---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
author: tfitzmac
ms.openlocfilehash: 8ccf2565d722a09de5f08ebe7333436729ce1b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346930"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса windowsEnrollmentStatusScreenSettings

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Параметр экрана состояния подачи заявок
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hideInstallationProgress|Boolean.|Показать или скрыть выполнения установки для пользователей|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean.|Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей|
|blockDeviceSetupRetryByUser|Boolean.|Пользователь может повторно запустите программу установки на сбой установки|
|allowLogCollectionOnInstallFailure|Boolean.|Разрешить или заблокировать семейства журнала на сбой установки|
|customErrorMessage|String.|Задать пользовательское сообщение об ошибке для отображения после сбоя установки|
|installProgressTimeoutInMinutes|Int32|Задать время ожидания ход выполнения установки в минутах|
|allowDeviceUseOnInstallFailure|Boolean.|Разрешает пользователю продолжить использование устройства на сбой установки|

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





