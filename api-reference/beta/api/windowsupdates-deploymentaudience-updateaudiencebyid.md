---
title: 'deploymentAudience: updateAudienceById'
description: Обновление семейство участников и исключения развертыванияAudience с помощью updatableAsset ресурсов того же типа.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: b2aaa550769a96d5f21cabe5f57b28578ff13736
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029953"
---
# <a name="deploymentaudience-updateaudiencebyid"></a>deploymentAudience: updateAudienceById

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление семейство участников и исключения [развертыванияAudience](../resources/windowsupdates-deploymentaudience.md) с помощью [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсов того же типа.

Добавление [azureADDevice](../resources/windowsupdates-azureaddevice.md) в собрания участников или исключения аудитории развертывания автоматически создает объект устройства Azure AD, если он еще не существует.

Если один и тот же [updatableAsset](../resources/windowsupdates-updatableasset.md)  будет включен в коллекции исключений и членов **развертыванияAudience,** развертывание не будет применяться к этому активу. 

Вы также можете использовать обновление [методаAudience](windowsupdates-deploymentaudience-updateaudience.md) для обновления **deploymentAudience.**

> [!NOTE]
> Этот API имеет [известные проблемы, связанные](/Graph/known-issues#accessing-and-updating-deployment-audiences) с развертываниями, созданными через Intune.

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
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|memberEntityType|String|Полный тип updatable активов. Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice`, `#microsoft.graph.windowsUpdates.updatableAssetGroup`.|
|addMembers|Коллекция String|Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве участников аудитории развертывания.|
|removeMembers|Коллекция String|Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве членов аудитории развертывания.|
|addExclusions|Коллекция String|Список идентификаторов, соответствующих updatable активам, которые необходимо добавить в качестве исключений из аудитории развертывания.|
|removeExclusions|Коллекция String|Список идентификаторов, соответствующих updatable активам, которые необходимо удалить в качестве исключений из аудитории развертывания.|



## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/deploymentaudience-updateaudiencebyid-go-snippets.md)]
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

