---
title: Тип ресурса Секуритибаселинесеттингстате
description: Состояние соответствия базовой безопасности параметру для устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522582"
---
# <a name="securitybaselinesettingstate-resource-type"></a>Тип ресурса Секуритибаселинесеттингстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия базовой безопасности параметру для устройства

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинесеттингстатес](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|Коллекция [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Список свойств и связей объектов [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Получение Секуритибаселинесеттингстате](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Чтение свойств и связей объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Создание Секуритибаселинесеттингстате](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Создание нового объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|
|[Удаление Секуритибаселинесеттингстате](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|Нет|Удаляет объект [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md).|
|[Обновление Секуритибаселинесеттингстате](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[Секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md)|Обновление свойств объекта [секуритибаселинесеттингстате](../resources/intune-deviceintent-securitybaselinesettingstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта|
|settingName|String|Имя параметра, о котором сообщается|
|state|[Секуритибаселинекомплианцестате](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Состояние соответствия параметру базового уровня безопасности. Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|Сеттингкатегорид|String|Идентификатор категории параметров, к которой относится этот параметр|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



