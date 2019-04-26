---
title: Тип ресурса Мобилеаппинсталлсуммари
description: Содержит свойства для сводки установки мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a981477daefae92b6afcd3612a173d75b37e8637
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551871"
---
# <a name="mobileappinstallsummary-resource-type"></a>Тип ресурса Мобилеаппинсталлсуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки установки мобильного приложения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Мобилеаппинсталлсуммари](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Чтение свойств и связей объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .|
|[Обновление Мобилеаппинсталлсуммари](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Обновление свойств объекта [мобилеаппинсталлсуммари](../resources/intune-apps-mobileappinstallsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installedDeviceCount|Int32|Количество устройств, на которых успешно установлено это приложение.|
|failedDeviceCount|Int32|Количество устройств, которые не удалось установить это приложение.|
|notApplicableDeviceCount|Int32|Количество устройств, неприменимых к этому приложению.|
|notInstalledDeviceCount|Int32|Количество устройств, на которых не установлено это приложение.|
|Пендингинсталлдевицекаунт|Int32|Количество устройств, которые были уведомлены об установке этого приложения.|
|installedUserCount|Int32|Количество пользователей, чьи устройства успешно выполнили установку этого приложения.|
|failedUserCount|Int32|Количество пользователей с 1 или больше устройств, которые не удалось установить это приложение.|
|notApplicableUserCount|Int32|Количество пользователей, чьи устройства были неприменимы к этому приложению.|
|notInstalledUserCount|Int32|Количество пользователей с 1 или больше устройств, которые не установили это приложение.|
|Пендингинсталлусеркаунт|Int32|Количество пользователей с 1 или больше устройств, которые были уведомлены об установке этого приложения и имеют 0 устройств с ошибками.|

## <a name="relationships"></a>Отношения
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





