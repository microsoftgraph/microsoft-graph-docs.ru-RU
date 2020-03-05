---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3758dd850a5c98ea2c0ddad4d261fc9a7388ac3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528227"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса Виндовсенроллментстатусскринсеттингс

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка экрана состояния регистрации

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|хидеинсталлатионпрогресс|Логический|Отображение или скрытие хода установки для пользователя|
|алловдевицеусебефорепрофилеандаппинсталлкомплете|Логический|Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений|
|блоккдевицесетупретрибюсер|Логический|Разрешить пользователю повторно выполнить установку при сбое установки|
|алловлогколлектиононинсталлфаилуре|Логический|Разрешение или блокировка сбора журналов при сбое установки|
|кустомеррормессаже|String|Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки|
|инсталлпрогресстимеаутинминутес|Int32|Задать время ожидания установки (в минутах)|
|алловдевицеусеонинсталлфаилуре|Логический|Разрешить пользователю продолжать использовать устройство при сбое установки|

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



