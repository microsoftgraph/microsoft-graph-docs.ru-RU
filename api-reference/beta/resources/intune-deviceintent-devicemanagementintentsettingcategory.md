---
title: Тип ресурса Девицеманажементинтентсеттингкатегори
description: Сущность, представляющая категорию параметров намерения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c22847e0f86a5f07655af3342a5e9ecd310d2681
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943286"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>Тип ресурса Девицеманажементинтентсеттингкатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая категорию параметров намерения


Наследуется от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентсеттингкатегориес](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|Коллекция [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Список свойств и связей объектов [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Получение Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Чтение свойств и связей объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Создание Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Создание нового объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Удаление Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|Нет|Удаляет объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).|
|[Обновление Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Обновление свойств объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор категории, наследуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|Строка|Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Сеттингдефинитионс|Коллекция [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров эта категория содержит унаследованные от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|settings|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Параметры, содержащиеся в этой категории|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```




