---
title: Тип ресурса Девицеманажементинтентсеттингкатегори
description: Сущность, представляющая категорию параметров намерения
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3765f120e3bda0bf8f41fa6e3d42ed557092d35b
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522561"
---
# <a name="devicemanagementintentsettingcategory-resource-type"></a>Тип ресурса Девицеманажементинтентсеттингкатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая категорию параметров намерения


НаСледуется от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтентсеттингкатегориес](../api/intune-deviceintent-devicemanagementintentsettingcategory-list.md)|Коллекция [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Список свойств и связей объектов [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Получение Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-get.md)|[Девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Чтение свойств и связей объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Создание Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-create.md)|[Девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Создание нового объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|
|[Удаление Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-delete.md)|Нет|Удаляет объект [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md).|
|[Обновление Девицеманажементинтентсеттингкатегори](../api/intune-deviceintent-devicemanagementintentsettingcategory-update.md)|[Девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)|Обновление свойств объекта [девицеманажементинтентсеттингкатегори](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор категории, наСледуемый от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|
|displayName|String|Имя категории, унаследованное от [девицеманажементсеттингкатегори](../resources/intune-deviceintent-devicemanagementsettingcategory.md)|

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







