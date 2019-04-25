---
title: Тип ресурса Виндовсманажементапфеалссуммари
description: Содержит свойства для сводки о работоспособности приложения управления Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aea7f113d144ca876b301acc3b303ac0f7072bc4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520027"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a>Тип ресурса Виндовсманажементапфеалссуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки о работоспособности приложения управления Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Виндовсманажементапфеалссуммари](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Чтение свойств и связей объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|
|[Обновление Виндовсманажементапфеалссуммари](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).|Обновление свойств объекта [виндовсманажементапфеалссуммари](../resources/intune-devices-windowsmanagementapphealthsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта сводки работоспособности приложения управления Windows.|
|Хеалсидевицекаунт|Int32|Работоспособное число устройств.|
|Унхеалсидевицекаунт|Int32|Неработоспособное число устройств.|
|unknownDeviceCount|Int32|Количество неИзвестных устройств.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```





