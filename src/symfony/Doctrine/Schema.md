## Schema 管理
- SchemaTool 根据Entity的metadata创建表

        public function createTable($number)
        {
            $metadata = $this->em->getClassMetadata(Log::class);

            $schemaTool = new \Doctrine\ORM\Tools\SchemaTool($this->locationEm);
            $metadata->setPrimaryTable(['name' => 'log_' . $number]);
            return $schemaTool->createSchema(array($metadata));
        }
- SchameManager 判断表是否存在

		public function logExist($number)
        {
            return $this->em->getConnection()->getSchemaManager()->tablesExist('log_' . $number);
        }