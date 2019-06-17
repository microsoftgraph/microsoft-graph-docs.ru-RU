---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22f7497fb79921bbbf34c6f3334ccc2ae4d7d53
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994904"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>Тип ресурса Виндовсенроллментстатусскринсеттингс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Настройка экрана состояния регистрации

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Хидеинсталлатионпрогресс|Boolean|Отображение или скрытие хода установки для пользователя|
|Алловдевицеусебефорепрофилеандаппинсталлкомплете|Boolean|Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений|
|Блоккдевицесетупретрибюсер|Boolean|Разрешить пользователю повторно выполнить установку при сбое установки|
|Алловлогколлектиононинсталлфаилуре|Boolean|Разрешение или блокировка сбора журналов при сбое установки|
|Кустомеррормессаже|String|Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки|
|Инсталлпрогресстимеаутинминутес|Int32|Задать время ожидания установки (в минутах)|
|Алловдевицеусеонинсталлфаилуре|Boolean|Разрешить пользователю продолжать использовать устройство при сбое установки|

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





