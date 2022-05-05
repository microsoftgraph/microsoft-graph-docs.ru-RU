---
title: 'sourceCollection: purgeData'
description: Используйте метод очистки данных для удаления конфиденциальных Microsoft Teams сообщений в sourceCollection.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: fa2bb5cb399d22302d167fd9fb120f13d43e3d43
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211441"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection: purgeData

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Окончательное удаление Microsoft Teams сообщений, содержащихся в [объекте sourceCollection](../resources//ediscovery-sourcecollection.md).

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
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

Если операция очистки данных успешно запущена, это действие возвращает код `202 Accepted` отклика. Ответ также будет содержать заголовок`Location`, содержащий расположение операции очистки данных, созданной для фиксации очистки.[](../resources/ediscovery-purgedataoperation.md)
Чтобы проверить состояние операции очистки данных, выполните запрос GET к URL-адресу расположения. После успешного завершения [запроса состояние](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) изменится на `succeeded`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollectionthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollectionthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollectionthispurgedata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollectionthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/sourcecollectionthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/sourcecollectionthispurgedata-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
