---
title: Тип ресурса windowsInformationProtectionAppLearningSummary
description: Объект сводки по обучению Windows Information Protection для приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cb2de8ba6b3a8daec7d13cb72a683bdec74e6c28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987701"
---
# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>Тип ресурса windowsInformationProtectionAppLearningSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект сводки по обучению Windows Information Protection для приложений.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-list.md)|Коллекция [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Список свойств и связей объектов [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).|
|[Получение объекта windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Чтение свойств и связей объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).|
|[Создание объекта windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).|
|[Удаление объекта windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-delete.md)|Нет|Удаляет объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).|
|[Обновление объекта windowsInformationProtectionAppLearningSummary](../api/intune-wip-windowsinformationprotectionapplearningsummary-update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)|Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.|
|applicationName|String|Имя приложения|
|applicationType|[applicationType](../resources/intune-wip-applicationtype.md)|Тип приложения. Возможные значения: `universal`, `desktop`.|
|deviceCount|Int32|Количество устройств|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```





