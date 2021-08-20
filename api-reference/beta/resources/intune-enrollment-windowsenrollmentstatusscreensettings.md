---
title: тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр состояния регистрации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0f483d4217506aa440df1108c968ba4df83f8fc7f55433e193d4c07388a70ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164218"
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
|blockDeviceSetupRetryByUser|Логический|Разрешить пользователю повторно повторить установку при сбое установки|
|allowLogCollectionOnInstallFailure|Логический|Разрешить или заблокировать коллекцию журналов при сбое установки|
|customErrorMessage|String|Настройка настраиваемой ошибки для демонстрации при сбое установки|
|installProgressTimeoutInMinutes|Int32|Установите время выполнения установки за несколько минут|
|allowDeviceUseOnInstallFailure|Логический|Разрешить пользователю продолжить использование устройства при сбое установки|

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




