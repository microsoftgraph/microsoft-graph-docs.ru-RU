---
title: 'sourceCollection: purgeData'
description: Используйте метод очистки данных для удаления конфиденциальных Microsoft Teams сообщений в sourceCollection.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a7a2e7ae0138f57739184325b2615d90d74d5abb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608425"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection: purgeData

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Постоянно удаляйте Microsoft Teams сообщения, содержащиеся в [sourceCollection](../resources//ediscovery-sourcecollection.md).

>**Примечание:** Этот запрос очищает Teams данных. Он не очищает другие типы данных, например элементы почтовых ящиков.

Вы можете собирать и очищать следующие категории Teams контента:
- **Teams 1:1** — сообщения чата, сообщения и вложения, Teams беседы между двумя людьми. Teams 1:1 чаты также *называются беседами*.
- **Teams групповых чатов** — сообщения чата, сообщения и вложения, Teams беседы между тремя или более людьми. Также *называются 1:N* чаты или *групповые беседы*.
- **Teams** - сообщения чата, сообщения, ответы и вложения, общие в стандартном Teams канале.
- **Частные каналы** — сообщения, ответы и вложения, общие в частном Teams канале.
- **Общие каналы** — сообщения, ответы и вложения, общие в общем Teams канале.

Дополнительные сведения о чистке Teams см.:
- [Серия решений по обнаружению электронных данных: сценарий утечки данных — поиск и очистка](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery для контента в Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 

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

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.

Если операция очистки данных успешно запущена, это действие возвращает код `202 Accepted` ответа. В ответе также будет содержаться `Location` заглавный загот, [](../resources/ediscovery-purgedataoperation.md) содержащий расположение операции очистки данных, созданной для совершения очистки.
Чтобы проверить состояние операции очистки данных, сделайте запрос GET на URL-адрес расположения. После успешного завершения запроса [состояние изменится](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) на `succeeded`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
