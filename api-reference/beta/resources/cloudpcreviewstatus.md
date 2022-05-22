---
title: Тип ресурса cloudPcReviewStatus
description: Представляет сведения о состоянии проверки облачного компьютера.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: efaaeeab9474ab785cba4f40e64794af6d3344fc
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629533"
---
# <a name="cloudpcreviewstatus-resource-type"></a>Тип ресурса cloudPcReviewStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о состоянии проверки облачного компьютера.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|azureStorageAccountId|Строка|Идентификатор ресурса учетной записи служба хранилища Azure, в которой сохраняется моментальный снимок облачного компьютера.|
|azureStorageAccountName|Строка|Имя учетной записи служба хранилища Azure, в которой сохраняется моментальный снимок облачного компьютера.|
|inReview|Логический| `True` Значение , если администратору задано значение "Облачный компьютер".|
|restorePointDateTime|DateTimeOffset|Конкретная дата и время создания моментального снимка облачного компьютера, который был создан и сохранен автоматически, если для облачного компьютера задано значение "Проверка". Метка времени отображается в формате ISO 8601 и времени в формате UTC. Например, полночь в формате UTC 1 января 2014 г. отображается как `2014-01-01T00:00:00Z`.|
|reviewStartDateTime|DateTimeOffset|Конкретная дата и время, когда облачный компьютер был настроен на проверку. Метка времени отображается в формате ISO 8601 и времени в формате UTC. Например, полночь в формате UTC 1 января 2014 г. отображается как `2014-01-01T00:00:00Z`.|
|subscriptionId|String|Идентификатор подписки Azure, в которой сохраняется моментальный снимок облачного компьютера, в формате GUID.|
|subscriptionName|Строка|Имя подписки Azure, в которой сохраняется моментальный снимок облачного компьютера.|
|userAccessLevel|[cloudPcUserAccessLevel](#cloudpcuseraccesslevel-values)|Уровень доступа конечного пользователя на облачном компьютере. Возможные значения: `unrestricted`, `restricted`.|

### <a name="cloudpcuseraccesslevel-values"></a>Значения cloudPcUserAccessLevel

|Элемент|Значение|Описание|
|:---|:---|:---|
|unrestricted|0|Без ограничений. Пользователи могут получить доступ к облачному компьютеру.|
|Ограничен|1|Пользователям не разрешен доступ к облачному компьютеру.|
|unknownFutureValue|999|Значение sentinel для развиваемого перечисления. Не следует использовать.|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcReviewStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcReviewStatus",
  "azureStorageAccountId": "String",
  "azureStorageAccountName": "String",
  "inReview": "Boolean",
  "restorePointDateTime": "String (timestamp)",
  "reviewStartDateTime": "String (timestamp)",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "userAccessLevel": "String"
}
```

