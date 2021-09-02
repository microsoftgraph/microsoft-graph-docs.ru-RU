---
title: тип ресурса companyPortalBlockedAction
description: Заблокированные действия на портале компании в зависимости от типов владения платформой и устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 099f0d5feaa5710cf4d78c3af006d0218c523fa1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805698"
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



