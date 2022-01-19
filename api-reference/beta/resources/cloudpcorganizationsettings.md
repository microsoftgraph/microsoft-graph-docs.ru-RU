---
title: тип ресурса cloudPcOrganizationSettings
description: Представляет параметры организации облачных ПК для клиента.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0a74f5db7c98cf5f6ec96d1fbddb5908f28ccea5
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072852"
---
# <a name="cloudpcorganizationsettings-resource-type"></a>тип ресурса cloudPcOrganizationSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры организации облачных ПК для клиента. У клиента есть только один **объект cloudPcOrganizationSettings.**

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-get.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcOrganizationSettings.](../resources/cloudpcorganizationsettings.md)|
|[Обновление cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-update.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Обновление свойств объекта [cloudPcOrganizationSettings.](../resources/cloudpcorganizationsettings.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID параметров организации.|
|osVersion|[cloudPcOperatingSystem](#cloudpcoperatingsystem-values)|Тип учетной записи пользователя на предварительных облачных компьютерах. Допустимые значения: `windows10`, `windows11`, `unknownFutureValue`.|
|userAccountType|[cloudPcUserAccountType](#cloudpcuseraccounttype-values)|Версия операционной системы (ОС) для обеспечения на облачных ПК. Допустимые значения: `standardUser`, `administrator`, `unknownFutureValue`.|

### <a name="cloudpcoperatingsystem-values"></a>значения cloudPcOperatingSystem

|Member|Описание|
|:---|:---|
|windows10|Операционная Windows 10.|
|windows11|Операционная Windows 11.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

### <a name="cloudpcuseraccounttype-values"></a>значения cloudPcUserAccountType

|Member|Описание|
|:---|:---|
|standardUser|Пользователь без локальных административных разрешений на облачном компьютере. Стандартные пользователи могут устанавливать контент только из приложения Microsoft Store, но они не могут изменять Windows параметров, которые требуют местных административных привилегий.|
|администратор|Пользователь с полными локальными административными разрешениями на облачном компьютере. Администраторы могут устанавливать любое программное обеспечение и изменять любой файл или параметр на облачном компьютере.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOrganizationSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOrganizationSettings",
  "id": "String (identifier)",
  "osVersion": "String",
  "userAccountType": "String"
}
```
