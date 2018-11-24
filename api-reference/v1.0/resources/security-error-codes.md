# <a name="microsoft-graph-security-api-error-responses"></a>Сообщения об ошибках API безопасности Microsoft Graph

Ошибки в Microsoft Graph API безопасности в Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и доставляются путем получения заголовка предупреждения.

API-Интерфейс безопасности Microsoft Graph — федеративных служба, которая получает несколько ответов от всех поставщиков данных. При получении ошибки HTTP с API-Интерфейс безопасности Microsoft Graph возвращается предупреждение заголовка в следующем формате:<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Этот заголовок предупреждение только отправляется обратно клиентов при один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404. Пример:

- HttpStatusCode.Forbidden (403) может быть возвращено, если не предоставляется доступ к ресурсу.
- Если поставщик времени ожидания, HttpStatusCode.GatewayTimeout (504) возвращается в заголовке предупреждения.
- Если происходит ошибка внутреннего поставщика HttpStatusCode.InternalServerError (500) используется в заголовке предупреждения.

Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждение так как эти коды для успеха или когда данные не найдены соответственно. В системе с федеративным 404 не найден ожидается как количество раз данные известно только один или несколько, но не для всех поставщиков.

## <a name="example"></a>Пример

Пользователь запрашивает `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Так как 404 и 200 ожидаемых условиях, предупреждение заголовка содержит следующие элементы: 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Примечание:** Каждого заголовка HTTP — это коллекция элементов, чтобы пользователи могли предупреждение заголовок перечислить и проверить все элементы.

## <a name="see-also"></a>См. также

Если у вас возникли неполадки с авторизацией, см в нашем [блоге](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).
