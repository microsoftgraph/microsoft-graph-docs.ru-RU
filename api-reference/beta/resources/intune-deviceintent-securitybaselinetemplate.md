---
title: Тип ресурса Секуритибаселинетемплате
description: Базовый шаблон безопасности учетной записи
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b572d3cc25943438f190a46fd23704a2eb6b7be3
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522344"
---
# <a name="securitybaselinetemplate-resource-type"></a>Тип ресурса Секуритибаселинетемплате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый шаблон безопасности учетной записи


НаСледуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинетемплатес](../api/intune-deviceintent-securitybaselinetemplate-list.md)|Коллекция [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md)|Список свойств и связей объектов [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Получение Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[Секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md)|Чтение свойств и связей объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Создание Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[Секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md)|Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Удаление Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|Нет|Удаляет объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).|
|[Обновление Секуритибаселинетемплате](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[Секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md)|Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|String|Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|settings|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция всех параметров, унаследованных этим шаблоном от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|Коллекция [девицеманажементтемплатесеттингкатегори](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Коллекция параметров категорий в шаблоне, унаследованных от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|Девицестатесуммари|[Секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Сводка по состоянию базового устройства безопасности|
|deviceStates|Коллекция [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Состояния основного устройства безопасности|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```







