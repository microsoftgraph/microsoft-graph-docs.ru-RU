---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978573"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса windowsEnrollmentStatusScreenSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Параметр экрана состояния подачи заявок
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hideInstallationProgress|Boolean|Показать или скрыть выполнения установки для пользователей|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей|
|blockDeviceSetupRetryByUser|Boolean|Пользователь может повторно запустите программу установки на сбой установки|
|allowLogCollectionOnInstallFailure|Boolean|Разрешить или заблокировать семейства журнала на сбой установки|
|customErrorMessage|String|Задать пользовательское сообщение об ошибке для отображения после сбоя установки|
|installProgressTimeoutInMinutes|Int32|Задать время ожидания ход выполнения установки в минутах|
|allowDeviceUseOnInstallFailure|Boolean|Разрешает пользователю продолжить использование устройства на сбой установки|

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





