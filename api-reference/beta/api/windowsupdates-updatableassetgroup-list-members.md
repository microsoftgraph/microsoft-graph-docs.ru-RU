---
title: Список updatable членов группы активов
description: Список участников ресурса updatableAssetGroup. Участники имеют тип azureADDevice.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 54c6cdad0f4da6e36df2e24be16c02bb3c1252bc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009261"
---
# <a name="list-updatable-asset-group-members"></a>Список updatable членов группы активов
Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список участников ресурса [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md) Участники имеют тип [azureADDevice.](../resources/windowsupdates-azureaddevice.md)

Эта операция ссылается на **свойство** навигации участников ресурса **updatableAssetGroup.** Чтобы ссылаться на свойство типа, полученное из [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип производных ресурсов в URL-адрес запроса, т.е. `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members` .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|WindowsUpdates.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .

Чтобы использовать параметр запроса для свойства, которое не унаследовано от [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса для свойства. Например, чтобы применить `$select` к свойству **ошибок** [azureADDevice,](../resources/windowsupdates-azureaddevice.md)используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-updatableasset-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "6d49dfaf-9c24-42f7-9628-c136e35774c8"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "1f61492e-4e34-4dee-904a-0d38299e76b2"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "bfe3c2d1-4cef-4952-8c5e-30d56ccf0cdc"
    }
  ]
}
```

