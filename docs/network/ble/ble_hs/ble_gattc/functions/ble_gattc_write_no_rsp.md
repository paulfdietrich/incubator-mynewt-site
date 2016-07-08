## <font color="#F2853F" style="font-size:24pt">ble\_gattc\_write\_no\_rsp</font>

```c
int
ble_gattc_write_no_rsp(uint16_t conn_handle, uint16_t attr_handle,
                       const void *value, uint16_t value_len)
```

### Description

Initiates GATT procedure: Write Without Response. 

### Parameters

| *Parameter* | *Description* |
|-------------|---------------|
| conn\_handle | The connection over which to execute the procedure. |
| attr\_handle | The handle of the characteristic value to write to. |
| value | The value to write to the characteristic. |
| value\_len | The number of bytes to write. |

### Returned values

| *Value* | *Condition* |
|---------|-------------|
| 0 | Success. |
| [BLE host core return code](../../ble_hs_return_codes/#return-codes-core) | Unexpected error. |