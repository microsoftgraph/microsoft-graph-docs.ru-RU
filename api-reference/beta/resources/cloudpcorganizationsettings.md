---
title: Тип ресурса cloudPcOrganizationSettings
description: Представляет параметры организации облачных компьютеров для клиента.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 770531c1d5bcf5dac870b2c341c9b20e2d723e66
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733187"
---
# <a name="cloudpcorganizationsettings-resource-type"></a>Тип ресурса cloudPcOrganizationSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры организации облачных компьютеров для клиента. У клиента есть только один **объект cloudPcOrganizationSettings** .

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-get.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Чтение свойств и связей объекта [cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) .|
|[Обновление cloudPcOrganizationSettings](../api/cloudpcorganizationsettings-update.md)|[cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md)|Обновление свойств объекта [cloudPcOrganizationSettings](../resources/cloudpcorganizationsettings.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметров организации.|
|osVersion|[cloudPcOperatingSystem](#cloudpcoperatingsystem-values)|Версия операционной системы (ОС) для подготовки на облачных компьютерах. Допустимые значения: `windows10`, `windows11`, `unknownFutureValue`.|
|userAccountType|[CloudPcUserAccountType](#cloudpcuseraccounttype-values)|Тип учетной записи пользователя на подготовленных облачных компьютерах. Допустимые значения: `standardUser`, `administrator`, `unknownFutureValue`.|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|Представляет параметры организации облачных компьютеров для клиента. У клиента есть только один **объект cloudPcOrganizationSettings** . Значение языка по умолчанию `en-US`.|

### <a name="cloudpcoperatingsystem-values"></a>Значения cloudPcOperatingSystem

|Member|Описание|
|:---|:---|
|windows10|Windows 10 операционной системы.|
|windows11|Windows 11 операционной системы.|
|unknownFutureValue|Значение sentinel для развиваемого перечисления. Не следует использовать.|

### <a name="cloudpcuseraccounttype-values"></a>Значения cloudPcUserAccountType

|Member|Описание|
|:---|:---|
|standardUser|Пользователь без разрешений локального администратора на облачном компьютере. Стандартные пользователи могут устанавливать содержимое только из Microsoft Store приложения, но не могут изменять Windows, для которых требуются права локального администратора.|
|Администратора|Пользователь с полными разрешениями локального администратора на облачном компьютере. Администраторы могут установить любое программное обеспечение и изменить любой файл или параметр на облачном компьютере.|
|unknownFutureValue|Значение sentinel для развиваемого перечисления. Не следует использовать.|

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
  "userAccountType": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```
