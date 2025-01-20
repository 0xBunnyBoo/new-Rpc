  bytes32[] memory dataFeedIds = new bytes32[](2);
  dataFeedIds[0] = bytes32("ETH");
  dataFeedIds[1] = bytes32("BTC");
  uint256[] memory values = getOracleNumericValuesFromTxMsg(dataFeedIds);
  uint256 ethPrice = values[0];
  uint256 btcPrice = values[1];
