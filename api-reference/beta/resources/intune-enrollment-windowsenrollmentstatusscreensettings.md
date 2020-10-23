---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 722f262688a35f6e14ae495f0e5cf5ee5976beb5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697513"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса Виндовсенроллментстатусскринсеттингс

Пространство имен: microsoft.graph

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
|кустомеррормессаже|Строка|Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки|
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





