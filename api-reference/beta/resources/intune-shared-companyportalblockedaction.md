---
title: тип ресурса companyPortalBlockedAction
description: Заблокированные действия на портале компании в зависимости от типов владения платформой и устройствами
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8b04ce4697d2ff24f28644908cf12764f8bd3d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039198"
---
# <a name="companyportalblockedaction-resource-type"></a>тип ресурса companyPortalBlockedAction

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Заблокированные действия на портале компании в зависимости от типов владения платформой и устройствами

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|платформа|[devicePlatformType](../resources/intune-wip-deviceplatformtype.md)|ОС устройства/платформа. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Тип владения устройствами. Возможные значения: `unknown`, `company`, `personal`.|
|action|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|Действие устройства. Возможные значения: `unknown`, `remove`, `reset`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```



