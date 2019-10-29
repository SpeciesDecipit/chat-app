## LabSession9, Artemii Bykov, DS01
rs.status():
```
{
	"set" : "rs0",
	"date" : ISODate("2019-10-29T16:59:46.950Z"),
	"myState" : 1,
	"term" : NumberLong(5),
	"syncingTo" : "",
	"syncSourceHost" : "",
	"syncSourceId" : -1,
	"heartbeatIntervalMillis" : NumberLong(2000),
	"majorityVoteCount" : 2,
	"writeMajorityCount" : 2,
	"optimes" : {
		"lastCommittedOpTime" : {
			"ts" : Timestamp(1572368377, 1),
			"t" : NumberLong(5)
		},
		"lastCommittedWallTime" : ISODate("2019-10-29T16:59:37.175Z"),
		"readConcernMajorityOpTime" : {
			"ts" : Timestamp(1572368377, 1),
			"t" : NumberLong(5)
		},
		"readConcernMajorityWallTime" : ISODate("2019-10-29T16:59:37.175Z"),
		"appliedOpTime" : {
			"ts" : Timestamp(1572368377, 1),
			"t" : NumberLong(5)
		},
		"durableOpTime" : {
			"ts" : Timestamp(1572368377, 1),
			"t" : NumberLong(5)
		},
		"lastAppliedWallTime" : ISODate("2019-10-29T16:59:37.175Z"),
		"lastDurableWallTime" : ISODate("2019-10-29T16:59:37.175Z")
	},
	"lastStableRecoveryTimestamp" : Timestamp(1572368327, 1),
	"lastStableCheckpointTimestamp" : Timestamp(1572368327, 1),
	"electionCandidateMetrics" : {
		"lastElectionReason" : "stepUpRequestSkipDryRun",
		"lastElectionDate" : ISODate("2019-10-29T16:21:16.270Z"),
		"termAtElection" : NumberLong(5),
		"lastCommittedOpTimeAtElection" : {
			"ts" : Timestamp(1572366075, 1),
			"t" : NumberLong(4)
		},
		"lastSeenOpTimeAtElection" : {
			"ts" : Timestamp(1572366075, 1),
			"t" : NumberLong(4)
		},
		"numVotesNeeded" : 2,
		"priorityAtElection" : 1,
		"electionTimeoutMillis" : NumberLong(10000),
		"priorPrimaryMemberId" : 1,
		"numCatchUpOps" : NumberLong(27017),
		"newTermStartDate" : ISODate("2019-10-29T16:21:17.110Z"),
		"wMajorityWriteAvailabilityDate" : ISODate("2019-10-29T16:21:18.141Z")
	},
	"members" : [
		{
			"_id" : 0,
			"name" : "172.31.30.203:27017",
			"ip" : "172.31.30.203",
			"health" : 1,
			"state" : 1,
			"stateStr" : "PRIMARY",
			"uptime" : 2398,
			"optime" : {
				"ts" : Timestamp(1572368377, 1),
				"t" : NumberLong(5)
			},
			"optimeDate" : ISODate("2019-10-29T16:59:37Z"),
			"syncingTo" : "",
			"syncSourceHost" : "",
			"syncSourceId" : -1,
			"infoMessage" : "",
			"electionTime" : Timestamp(1572366076, 1),
			"electionDate" : ISODate("2019-10-29T16:21:16Z"),
			"configVersion" : 3,
			"self" : true,
			"lastHeartbeatMessage" : ""
		},
		{
			"_id" : 1,
			"name" : "db2:27017",
			"ip" : "172.31.21.96",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 2252,
			"optime" : {
				"ts" : Timestamp(1572368377, 1),
				"t" : NumberLong(5)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572368377, 1),
				"t" : NumberLong(5)
			},
			"optimeDate" : ISODate("2019-10-29T16:59:37Z"),
			"optimeDurableDate" : ISODate("2019-10-29T16:59:37Z"),
			"lastHeartbeat" : ISODate("2019-10-29T16:59:45.151Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-29T16:59:46.441Z"),
			"pingMs" : NumberLong(0),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "db3:27017",
			"syncSourceHost" : "db3:27017",
			"syncSourceId" : 2,
			"infoMessage" : "",
			"configVersion" : 3
		},
		{
			"_id" : 2,
			"name" : "db3:27017",
			"ip" : "172.31.37.90",
			"health" : 1,
			"state" : 2,
			"stateStr" : "SECONDARY",
			"uptime" : 2397,
			"optime" : {
				"ts" : Timestamp(1572368377, 1),
				"t" : NumberLong(5)
			},
			"optimeDurable" : {
				"ts" : Timestamp(1572368377, 1),
				"t" : NumberLong(5)
			},
			"optimeDate" : ISODate("2019-10-29T16:59:37Z"),
			"optimeDurableDate" : ISODate("2019-10-29T16:59:37Z"),
			"lastHeartbeat" : ISODate("2019-10-29T16:59:45.151Z"),
			"lastHeartbeatRecv" : ISODate("2019-10-29T16:59:45.149Z"),
			"pingMs" : NumberLong(0),
			"lastHeartbeatMessage" : "",
			"syncingTo" : "172.31.30.203:27017",
			"syncSourceHost" : "172.31.30.203:27017",
			"syncSourceId" : 0,
			"infoMessage" : "",
			"configVersion" : 3
		}
	],
	"ok" : 1,
	"$clusterTime" : {
		"clusterTime" : Timestamp(1572368377, 1),
		"signature" : {
			"hash" : BinData(0,"AAAAAAAAAAAAAAAAAAAAAAAAAAA="),
			"keyId" : NumberLong(0)
		}
	},
	"operationTime" : Timestamp(1572368377, 1)
}
```
rs.config():
```
{
	"_id" : "rs0",
	"version" : 3,
	"protocolVersion" : NumberLong(1),
	"writeConcernMajorityJournalDefault" : true,
	"members" : [
		{
			"_id" : 0,
			"host" : "172.31.30.203:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {

			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 1,
			"host" : "db2:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {

			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		},
		{
			"_id" : 2,
			"host" : "db3:27017",
			"arbiterOnly" : false,
			"buildIndexes" : true,
			"hidden" : false,
			"priority" : 1,
			"tags" : {

			},
			"slaveDelay" : NumberLong(0),
			"votes" : 1
		}
	],
	"settings" : {
		"chainingAllowed" : true,
		"heartbeatIntervalMillis" : 2000,
		"heartbeatTimeoutSecs" : 10,
		"electionTimeoutMillis" : 10000,
		"catchUpTimeoutMillis" : -1,
		"catchUpTakeoverDelayMillis" : 30000,
		"getLastErrorModes" : {

		},
		"getLastErrorDefaults" : {
			"w" : 1,
			"wtimeout" : 0
		},
		"replicaSetId" : ObjectId("5db8408f835c699263ddd99a")
	}
}
```