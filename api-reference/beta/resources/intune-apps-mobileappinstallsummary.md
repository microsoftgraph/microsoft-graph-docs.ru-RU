---
title: тип ресурса mobileAppInstallSummary
description: Содержит свойства для сводки установки мобильного приложения.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1cc168933bad8a1eef5e177cc5361dd196c31cb5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124233"
---
# <a name="mobileappinstallsummary-resource-type"></a>тип ресурса mobileAppInstallSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки установки мобильного приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Чтение свойств и связей объекта [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)|
|[Обновление mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Обновление свойств объекта [mobileAppInstallSummary.](../resources/intune-apps-mobileappinstallsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installedDeviceCount|Int32|Количество устройств, успешно установленных в этом приложении.|
|failedDeviceCount|Int32|Количество устройств, которые не смогли установить это приложение.|
|notApplicableDeviceCount|Int32|Количество устройств, которые не применимы для этого приложения.|
|notInstalledDeviceCount|Int32|Количество устройств, на которые не установлено это приложение.|
|pendingInstallDeviceCount|Int32|Количество устройств, которые были уведомлены об установке этого приложения.|
|installedUserCount|Int32|Число пользователей, устройства которых успешно установили это приложение.|
|failedUserCount|Int32|Число пользователей, у них есть 1 или более устройств, которые не смогли установить это приложение.|
|notApplicableUserCount|Int32|Число пользователей, устройства которых не были применимы к этому приложению.|
|notInstalledUserCount|Int32|Число пользователей с 1 или более устройствами, которые не установили это приложение.|
|pendingInstallUserCount|Int32|Число пользователей с 1 или более устройствами, которые были уведомлены об установке этого приложения, и имеют 0 устройств с ошибками.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```



