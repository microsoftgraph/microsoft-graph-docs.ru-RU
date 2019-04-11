---
title: Тип ресурса Девицеманажементтемплатесеттингкатегори
description: Сущность, представляющая категорию параметров шаблона
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f8974c102bcd07bb6042e703f38b59840a164b6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807254"
---
# <a name="devicemanagementtemplatesettingcategory-resource-type"></a>Тип ресурса Девицеманажементтемплатесеттингкатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая категорию параметров шаблона


НаСледуется от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементтемплатесеттингкатегориес](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-list.md)|Коллекция [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Список свойств и связей объектов [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .|
|[Получение Девицеманажементтемплатесеттингкатегори](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Чтение свойств и связей объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .|
|[Создание Девицеманажементтемплатесеттингкатегори](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-create.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Создание нового объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .|
|[Удаление Девицеманажементтемплатесеттингкатегори](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-delete.md)|Нет|Удаляет объект [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md).|
|[Обновление Девицеманажементтемплатесеттингкатегори](../api/intune-deviceintent-devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Обновление свойств объекта [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор категории, наСледуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|String|Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Сеттингдефинитионс|Коллекция [девицеманажементсеттингдефинитион](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|Определения параметров эта категория содержит унаследованные от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|Рекоммендедсеттингс|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Параметры, содержащиеся в этой категории|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplateSettingCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```





