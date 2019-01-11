---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877450"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса windowsEnrollmentStatusScreenSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Параметр экрана состояния подачи заявок
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hideInstallationProgress|Логический|Показать или скрыть выполнения установки для пользователей|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Логический|Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей|
|blockDeviceSetupRetryByUser|Логический|Пользователь может повторно запустите программу установки на сбой установки|
|allowLogCollectionOnInstallFailure|Логический|Разрешить или заблокировать семейства журнала на сбой установки|
|customErrorMessage|Строка|Задать пользовательское сообщение об ошибке для отображения после сбоя установки|
|installProgressTimeoutInMinutes|Int32|Задать время ожидания ход выполнения установки в минутах|
|allowDeviceUseOnInstallFailure|Логический|Разрешает пользователю продолжить использование устройства на сбой установки|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





