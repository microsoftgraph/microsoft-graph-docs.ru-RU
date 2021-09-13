---
title: тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр состояния регистрации
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7578f25bf3ed2ed8b47d6cb7c039fd6bda7b89a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039898"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>тип ресурса windowsEnrollmentStatusScreenSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметр состояния регистрации

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|hideInstallationProgress|Логический|Показать пользователю или скрыть ход установки|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Логический|Разрешить или заблокировать использование устройства перед завершением установки профиля и приложения|
|blockDeviceSetupRetryByUser|Логическое|Разрешить пользователю повторно повторить установку при сбое установки|
|allowLogCollectionOnInstallFailure|Логическое|Разрешить или заблокировать коллекцию журналов при сбое установки|
|customErrorMessage|String|Настройка настраиваемой ошибки для демонстрации при сбое установки|
|installProgressTimeoutInMinutes|Int32|Установите время выполнения установки за несколько минут|
|allowDeviceUseOnInstallFailure|Логическое|Разрешить пользователю продолжить использование устройства при сбое установки|

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



