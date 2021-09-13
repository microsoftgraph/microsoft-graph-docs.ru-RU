---
title: тип ресурса deviceManagementCollectionSettingInstance
description: Экземпляр параметра, представляющий коллекцию значений
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f652e26a958abee9a8f1423013bd5e733ec5e5d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134985"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a>тип ресурса deviceManagementCollectionSettingInstance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий коллекцию значений


Наследует [от deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementCollectionSettingInstances](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|[коллекция deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Список свойств и связей [объектов deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|
|[Get deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Чтение свойств и связей [объекта deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|
|[Создание deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Создание нового [объекта deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|
|[Удаление deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|Нет|Удаляет [устройствоManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).|
|[Обновление deviceManagementCollectionSettingInstance](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Обновление свойств объекта [deviceManagementCollectionSettingInstance.](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|definitionId|String|ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|valueJson|String|Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|значение|[коллекция deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция значений|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



