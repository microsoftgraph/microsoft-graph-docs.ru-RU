---
title: тип ресурса configManagerPolicySummary
description: Сводка политики ConfigManager.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 88c31f9314f7cc4c55c68b328768e3119d913298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033457"
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



