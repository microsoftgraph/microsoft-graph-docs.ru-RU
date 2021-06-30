---
title: тип ресурса teamworkApplicationIdentity
description: Представляет приложение в Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b7e6c17b70e7f30e102e270d2d98b406e01dcae3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211386"
---
# <a name="teamworkapplicationidentity-resource-type"></a>тип ресурса teamworkApplicationIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение **в** Microsoft Teams. `teamworkApplicationIdentity` используется для представления ботов и исходяющих веб-@mentioned в сообщениях.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|applicationIdentityType|teamworkApplicationIdentityType| Тип ссылаемого приложения. Возможные значения: `aadApplication` `bot` , , , , `tenantBot` и `office365Connector` `outgoingWebhook` .|
|displayName|String|Унаследованный от [удостоверения](../resources/identity.md). Отображение имени приложения. Необязательно.|
|id|String|Унаследованный от [удостоверения](../resources/identity.md). ID приложения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkApplicationIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkApplicationIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "applicationIdentityType": "String"
}
```

