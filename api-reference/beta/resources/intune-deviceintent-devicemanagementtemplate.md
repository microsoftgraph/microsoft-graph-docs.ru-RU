---
title: Тип ресурса Девицеманажементтемплате
description: Объект, представляющий определенную коллекцию параметров устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cf144ed30a017dc1f3ae84fc481568adc0d0d09
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522519"
---
# <a name="devicemanagementtemplate-resource-type"></a>Тип ресурса Девицеманажементтемплате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий определенную коллекцию параметров устройства

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементтемплатес](../api/intune-deviceintent-devicemanagementtemplate-list.md)|Коллекция [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Список свойств и связей объектов [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Получение Девицеманажементтемплате](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[Девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Чтение свойств и связей объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Создание Девицеманажементтемплате](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[Девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Удаление Девицеманажементтемплате](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|Нет|Удаляет объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md).|
|[Обновление Девицеманажементтемплате](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[Девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|Обновление свойств объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[действие createInstance](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[Девицеманажементинтент](../resources/intune-deviceintent-devicemanagementintent.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор шаблона|
|displayName|String|Отображаемое имя шаблона|
|description|String|Описание шаблона|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|settings|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров, которые содержит этот шаблон|
|categories|Коллекция [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Коллекция настроек категорий в шаблоне|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```







