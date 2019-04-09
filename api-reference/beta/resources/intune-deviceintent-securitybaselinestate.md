---
title: Тип ресурса Секуритибаселинестате
description: Состояние базового уровня безопасности для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524563"
---
# <a name="securitybaselinestate-resource-type"></a>Тип ресурса Секуритибаселинестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние базового уровня безопасности для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинестатес](../api/intune-deviceintent-securitybaselinestate-list.md)|Коллекция [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md)|Список свойств и связей объектов [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Получение Секуритибаселинестате](../api/intune-deviceintent-securitybaselinestate-get.md)|[Секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md)|Чтение свойств и связей объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Создание Секуритибаселинестате](../api/intune-deviceintent-securitybaselinestate-create.md)|[Секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md)|Создание нового объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .|
|[Удаление Секуритибаселинестате](../api/intune-deviceintent-securitybaselinestate-delete.md)|Нет|Удаляет объект [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md).|
|[Обновление Секуритибаселинестате](../api/intune-deviceintent-securitybaselinestate-update.md)|[Секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md)|Обновление свойств объекта [секуритибаселинестате](../resources/intune-deviceintent-securitybaselinestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|Секуритибаселинетемплатеид|String|Идентификатор шаблона базовой безопасности|
|displayName|String|Отображаемое имя базового плана безопасности|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|settingStates|Коллекция [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Состояние базового уровня безопасности для различных параметров устройства|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



