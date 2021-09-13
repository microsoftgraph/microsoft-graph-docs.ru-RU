---
title: тип ресурса officeClientConfigurationAssignment
description: Office Назначение конфигурации клиента.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1aaec0c15f87167d3fe5b471e795f5ae56d59c9d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111343"
---
# <a name="officeclientconfigurationassignment-resource-type"></a>тип ресурса officeClientConfigurationAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Office Назначение конфигурации клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список officeClientConfigurationAssignments](../api/intune-cirrus-officeclientconfigurationassignment-list.md)|[коллекция officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список свойств и связей [объектов officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)|
|[Get officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-get.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Чтение свойств и связей [объекта officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)|
|[Создание officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-create.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Создание нового [объекта officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)|
|[Удаление officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-delete.md)|Нет|Удаляет [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).|
|[Обновление officeClientConfigurationAssignment](../api/intune-cirrus-officeclientconfigurationassignment-update.md)|[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Обновление свойств объекта [officeClientConfigurationAssignment.](../resources/intune-cirrus-officeclientconfigurationassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id of the OfficeConfigurationAssignment.|
|target|[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|Целевое назначение, определенное администратором.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



