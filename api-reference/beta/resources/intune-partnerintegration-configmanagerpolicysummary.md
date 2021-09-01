---
title: тип ресурса configManagerPolicySummary
description: Сводка политики ConfigManager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2cdb8393bd791af124232c2be3b35ede171bcf50
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805305"
---
# <a name="configmanagerpolicysummary-resource-type"></a>тип ресурса configManagerPolicySummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка политики ConfigManager.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|targetedDeviceCount|Int32|Количество устройств, на которые ориентирована политика.|
|compliantDeviceCount|Int32|Количество устройств, которые оцениваются как совместимые с политикой.|
|nonCompliantDeviceCount|Int32|Количество устройств, несовершенных политикой.|
|failedDeviceCount|Int32|Количество устройств, которые не были оценены политикой.|
|pendingDeviceCount|Int32|Количество устройств, которые признали политику, но находятся в ожидании оценки.|
|enforcedDeviceCount|Int32|Количество устройств, исправленных политикой.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configManagerPolicySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerPolicySummary",
  "targetedDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "enforcedDeviceCount": 1024
}
```



