---
title: Тип ресурса Конфигманажерполицисуммари
description: Сводка по политике Конфигманажер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63e85448b70abc76f4df0021c4f5516e778ebe0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302011"
---
# <a name="configmanagerpolicysummary-resource-type"></a>Тип ресурса Конфигманажерполицисуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по политике Конфигманажер.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|таржетеддевицекаунт|Int32|Количество устройств, для которых предназначена политика.|
|compliantDeviceCount|Int32|Количество устройств, которые оцениваются в соответствии с политикой.|
|nonCompliantDeviceCount|Int32|Количество устройств, которые оцениваются не в соответствии с политикой.|
|failedDeviceCount|Int32|Количество устройств, которые не удалось оценить с помощью политики.|
|пендингдевицекаунт|Int32|Количество устройств, которые подтвердили политику, но ожидают оценки.|
|енфорцеддевицекаунт|Int32|Количество устройств, исправленных политикой.|

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




