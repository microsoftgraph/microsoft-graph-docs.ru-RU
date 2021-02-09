---
title: Тип enum advancedBitLockerState
description: Состояние Advanced BitLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ad93a61e03e923ef1c74121574ee5f4e9a94d36
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153601"
---
# <a name="advancedbitlockerstate-enum-type"></a>Тип enum advancedBitLockerState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние Advanced BitLocker

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|success|0|Advanced BitLocker State Success|
|noUserConsent|1 |Пользователь не предоставил согласие на шифрование|
|osVolumeUnprotected|2 |Обнаружен незащищаемый том ОС|
|osVolumeTpmRequired|4 |TPM не используется для защиты тома ОС, но требуется политикой|
|osVolumeTpmOnlyRequired|8 |Защита TPM не используется только для тома ОС, но требуется политикой|
|osVolumeTpmPinRequired|16 |Защита TPM+PIN-кодов не используется для тома ОС, но требуется политикой|
|osVolumeTpmStartupKeyRequired|32|TPM+Защита ключа запуска не используется для тома ОС, но требуется политикой|
|osVolumeTpmPinStartupKeyRequired|64|TPM+ПИН-код и ключ запуска не используются для тома ОС, но требуются политикой|
|osVolumeEncryptionMethodMismatch|128|Метод шифрования тома ОС отличается от метода, установленного политикой|
|recoveryKeyBackupFailed|256|Сбой резервного копирования ключа восстановления|
|fixedDriveNotEncrypted|512|Фиксированный диск не зашифрован|
|fixedDriveEncryptionMethodMismatch|1024|Метод шифрования фиксированного диска отличается от метода шифрования, установленного политикой|
|loggedOnUserNonAdmin|2048|Во время входа пользователь не является администратором. Для этого требуется, чтобы для политики AllowStandardUserEncryption было установлено 1|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE не настроен|
|tpmNotAvailable|8192|TPM не доступен для BitLocker. Это означает, что TPM отсутствует, или переопределение недоступного реестра TPM задано или ОС хоста находится на переносимом диске или на диске с возможностью переноса.|
|tpmNotReady|16384|TPM не готов для BitLocker|
|networkError|32768|Сеть недоступна. Это необходимо для резервного копирования ключа восстановления. Это сообщается для устройств с шифрованием диска|




