---
title: Тип перечисления resultantAppStateDetail
description: Перечисление, указывающее дополнительные детали почему приложение имеет определенный установить состояние.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410240"
---
# <a name="resultantappstatedetail-enum-type"></a>Тип перечисления resultantAppStateDetail

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Перечисление, указывающее дополнительные детали почему приложение имеет определенный установить состояние.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noAdditionalDetails|0|Нет дополнительных сведений о доступны.|
|seeInstallErrorCode|2000|Сбой при установке приложения. Свойству код ошибки для получения дополнительных сведений см.|
|seeUninstallErrorCode|4000|Не удалось удалить приложение. Свойству код ошибки для получения дополнительных сведений см.|
|pendingReboot|5000|Устройства необходимо перезагрузить компьютер для завершения установки приложения.|
|platformNotApplicable|-1006|Приложение не применяется к этой платформе. (например приложения для Android нацелено на IOS)|
|minimumCpuSpeedNotMet|-1005|Скорость ЦП на целевом устройстве меньше, чем настроенные как минимум.|
|minimumLogicalProcessorCountNotMet|-1004|Количество логических процессоров на целевом устройстве меньше, чем настроенные как минимум.|
|minimumPhysicalMemoryNotMet|-1003|Объем ОЗУ на целевом устройстве меньше, чем настроенные как минимум.|
|minimumOsVersionNotMet|-1002|Версия операционной системы на целевом устройстве меньше, чем настроенные как минимум.|
|minimumDiskSpaceNotMet|-1001|Объем свободного места на устройстве конечного меньше, чем настроенные как минимум.|
|processorArchitectureNotApplicable|-1000|Архитектура устройство (например x86/amd64) не применимо для приложения.|




