---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80d869c3d80e7c164808147f732bf58bf5c1a15a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998856"
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





