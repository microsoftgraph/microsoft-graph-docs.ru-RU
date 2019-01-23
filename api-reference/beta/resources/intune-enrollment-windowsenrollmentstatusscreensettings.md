---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399936"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса windowsEnrollmentStatusScreenSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр экрана состояния подачи заявок

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hideInstallationProgress|Логический|Показать или скрыть выполнения установки для пользователей|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Логический|Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей|
|blockDeviceSetupRetryByUser|Логический|Пользователь может повторно запустите программу установки на сбой установки|
|allowLogCollectionOnInstallFailure|Логический|Разрешить или заблокировать семейства журнала на сбой установки|
|customErrorMessage|String|Задать пользовательское сообщение об ошибке для отображения после сбоя установки|
|installProgressTimeoutInMinutes|Int32|Задать время ожидания ход выполнения установки в минутах|
|allowDeviceUseOnInstallFailure|Логический|Разрешает пользователю продолжить использование устройства на сбой установки|

## <a name="relationships"></a>Отношения
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




