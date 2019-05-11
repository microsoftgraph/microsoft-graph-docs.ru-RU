---
title: Тип ресурса Девицеманажементдериведкредентиалсеттингс
description: Сущность, описывающая параметры уровня клиента для производных учетных данных
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fa7adfa76482cd4c67c2c3faaaf96b760f44bd2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957105"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>Тип ресурса Девицеманажементдериведкредентиалсеттингс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая параметры уровня клиента для производных учетных данных

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицеманажементдериведкредентиалсеттингс](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[Девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Чтение свойств и связей объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .|
|[Обновление Девицеманажементдериведкредентиалсеттингс](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[Девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Обновление свойств объекта [девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для производных учетных данных|
|helpUrl|Строка|URL-адрес, который будет доступен конечным пользователям для получения производных учетных данных с помощью корпоративного портала.|
|displayName|Строка|Отображаемое имя профиля.|
|имени|[Девицеманажементдериведкредентиалиссуер](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|Производный поставщик учетных данных, который будет использоваться. Возможные значения: `intercede`, `entrustDatacard`, `purebred`.|
|notificationType|[Девицеманажементдериведкредентиалнотификатионтипе](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|Методы, используемые для информирования конечного пользователя об открытии корпоративного портала для доставки в сеть Wi-Fi, VPN или профилей электронной почты, использующих сертификаты для устройства. Возможные значения: `none`, `companyPortal`, `email`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```




