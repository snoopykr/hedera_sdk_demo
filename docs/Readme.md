## account_allowance
- Alice의 Hbar를 Bob이 전송할수 있게 권한을 설정한다.
- 권한을 설정할때 Hbar 갯수도 지정하는데 이 이상 권한을 행사핧수가 없다.
## account_create_token_transfer
- 토큰이 아닌 Hbar를 전송한다.
- 새로 어카운트를 생성하고 Hbar를 전송한 후  hollow account(빈 계정)을 사용해서 계정 정보를 추룰한다.
- public key가 있는 정보와 없는 정보로 구분해서 추출한다.
## account_create_with_hts
- Sample 1 : NFT 생성하고, 민팅하고, 새로운 alias 어카운트를 생성하고, 전송을 한후, NFT 소유자 정보를 통해 어카운트 정보를 추출한다.
- Sample 2 : Token 생성하고, 새로운 alias 어카운트를 생성하고, 전송을 한후, 전송된 발란스를 사용해서 어카운트 정보를 추출한다.
## alias_id_example
- 새로운 alias 어카운트를 생성하고 Hbar를 전송
## consensus_pub_sub
- 16초 내에서 topic를 생성한다.
## consensus_pub_sub_chunked
- topic 생성인데...
에러 발생
```
for topic 0.0.3571695
wait to propagate...
panic: interface conversion: interface {} is hedera.TransactionResponse, not *services.Response

goroutine 1 [running]:
github.com/hashgraph/hedera-sdk-go/v2.(*TransactionReceiptQuery).Execute(0xc0002a61a0, 0xc00022fb00)
        /Users/snoopy_kr/Apps/Go/pkg/mod/github.com/hashgraph/hedera-sdk-go/v2@v2.34.1/transaction_receipt_query.go:138 +0x4d0
github.com/hashgraph/hedera-sdk-go/v2.TransactionResponse.GetReceipt({{0x0, 0x0, 0x0, 0x0}, {0x0, 0x0, 0x0, 0x0}, {0x0, 0x0, ...}, ...}, ...)
        /Users/snoopy_kr/Apps/Go/pkg/mod/github.com/hashgraph/hedera-sdk-go/v2@v2.34.1/transaction_response.go:58 +0x3c5
main.main()
        /Users/snoopy_kr/Working/GoLand/hedera_sdk_demo/consensus_pub_sub_chunked/main.go:149 +0x1025

Process finished with the exit code 2
```
## consensus_pub_sub_with_submit_key
- 새로운 어카운트 생성, 토픽 생성. 토픽을 구독한다.
## construct_client
## contract_helper
## create_account
## create_account_with_alias
## create_account_with_alias_and_receiver_signature_required
## create_account_with_threshold_keys
## create_file
## create_simple_contract
## create_stateful_contract
## custom_fees
## delete_account
## delete_file
## docs 
## dot_env
## exempt_custom_fees
## file_append_chunked
## generate_key
## generate_key_with_mnemonic
## get_account_balance
## get_address_book
## get_file_contents
## go.mod
## go.sum
## logging
## multi_app_transfer
## precompile_example
## rng_transaction
## schedule_identical_transaction
## schedule_multisig_transaction
## schedule_transfer_example
## schedule_with_expiration
## serialize-deserialize
## staking
## staking_with_update
## topic_with_admin_key
## transfer_crypto
## transfer_tokens
## update_account_public_key
## zero_token_operations