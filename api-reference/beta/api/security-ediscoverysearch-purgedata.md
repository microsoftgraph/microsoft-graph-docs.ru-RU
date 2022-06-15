---
title: 'ediscoverySearch: purgeData'
description: Используйте метод очистки данных для Teams сообщений в поиске eDiscovery.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f8ac399b59473a4c5ec1d1e1f064532228c23ea5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095407"
---
# <a name="ediscoverysearch-purgedata"></a>ediscoverySearch: purgeData
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Окончательное удаление Microsoft Teams сообщений, содержащихся в поиске [обнаружения электронных данных](../resources/security-ediscoverysearch.md).

>**Примечание:** Этот запрос очищает только Teams данных. Он не очищает другие типы данных, такие как элементы почтовых ящиков.

Вы можете собирать и очищать следующие категории Teams контента:
- **Teams 1:1** — сообщения чата, записи и вложения, Teams беседы между двумя людьми. Teams чаты 1:1 также *называются беседами*.
- **Teams чатов** — сообщения чата, записи и вложения, Teams беседы между тремя или несколькими пользователями. Также называется *1:N* чатами или *групповыми беседами*.
- **Teams каналов** — сообщения чата, записи, ответы и вложения, общие в стандартном Teams канале.
- **Частные каналы** — сообщения, ответы и вложения, общие в частном Teams канале.
- **Общие каналы —** сообщения, ответы и вложения, общие в общем Teams канале.

Дополнительные сведения об очистке Teams сообщений см. в следующих статьях:
- [Серия решений для обнаружения электронных данных: сценарий утечки данных — поиск и очистка](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery рабочего процесса для содержимого в Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/purgeData
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

Если операция очистки данных успешно запущена, это действие возвращает код `202 Accepted` отклика. Ответ также будет содержать заголовок`Location`, содержащий расположение операции очистки данных, созданной для фиксации очистки.[](../resources/security-ediscoverypurgedataoperation.md)
Чтобы проверить состояние операции очистки данных, выполните запрос GET к URL-адресу расположения.


## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverysearchthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverysearchthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverysearchthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoverysearchthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
