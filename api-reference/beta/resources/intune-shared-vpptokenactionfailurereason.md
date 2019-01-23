---
title: Тип перечисления vppTokenActionFailureReason
description: Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393146"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>Тип перечисления vppTokenActionFailureReason

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные типы причины возник сбой маркеров действие программы покупки корпоративного Apple.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Нет.|
|appleFailure|1|Произошла ошибка службы Apple.|
|internalError|2|Возникла внутренняя ошибка.|
|expiredVppToken|3|Произошла ошибка, так как истекших маркер покупки программы корпоративного Apple.|
|expiredApplePushNotificationCertificate|4|Произошла ошибка истечения срока действия сертификата Push-уведомления Apple тома покупки программы.|




