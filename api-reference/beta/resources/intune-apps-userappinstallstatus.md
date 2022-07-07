---
title: Тип ресурса userAppInstallStatus
description: Содержит свойства для состояния установки пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1063adfb3517e32b1190d7e59f03ae2d2740c1f
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668554"
---
# <a name="userappinstallstatus-resource-type"></a>Тип ресурса userAppInstallStatus

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов userAppInstallStatuse](../api/intune-apps-userappinstallstatus-list.md)|[Коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список свойств и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Получение userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Чтение свойств и связей объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Создание userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Создайте объект [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Удаление userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Нет|Удаляет [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Обновление userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Обновление свойств объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-apps-mobileapp.md);|Навигационная ссылка на мобильное приложение.|
|deviceStatuses|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Состояние установки приложения на устройствах.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```




