---
title: расширенный тип enumBitLockerState
description: Состояние Advanced BitLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bffc66ff77c74986b51a48f5c8f10ca05eb2406
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816573"
---
# <a name="advancedbitlockerstate-enum-type"></a>расширенный тип enumBitLockerState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние Advanced BitLocker

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|success|0|Расширенный успех состояния BitLocker|
|noUserConsent|1|Пользователь никогда не давал согласия на шифрование|
|osVolumeUnprotected|2|Обнаружен незащищаемый том ОС|
|osVolumeTpmRequired|4 |TPM не используется для защиты тома ОС, но требуется политикой|
|osVolumeTpmOnlyRequired|8 |Защита TPM только не используется для объема ОС, но требуется политикой|
|osVolumeTpmPinRequired|16 |Защита TPM+PIN не используется для объема ОС, но требуется политикой|
|osVolumeTpmStartupKeyRequired|32|Защита ключа TPM+Startup, не используемая для объема ОС, но требуется политикой|
|osVolumeTpmPinStartupKeyRequired|64|Ключ TPM+PIN+Startup, не используемый для объема ОС, но требуется политикой|
|osVolumeEncryptionMethodMismatch|128|Метод шифрования тома ОС отличается от метода, установленного политикой|
|recoveryKeyBackupFailed|256|Резервное копирование ключа восстановления не удалось|
|fixedDriveNotEncrypted|512|Фиксированный диск не шифруется|
|fixedDriveEncryptionMethodMismatch|1024|Метод шифрования фиксированного диска отличается от метода, установленного политикой|
|loggedOnUserNonAdmin|2048|Вход в систему пользователя не является администратором. Для этого требуется политика AllowStandardUserEncryption, установленная до 1|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE не настроен|
|tpmNotAvailable|8192|TPM не доступен для BitLocker. Это означает, что TPM отсутствует, или переопределение недоступного реестра TPM задано или осмий хост находится на портативном/римском диске.|
|tpmNotReady|16384|TPM не готова для BitLocker|
|networkError|32768|Сеть недоступна. Это необходимо для резервного копирования ключа восстановления. Это сообщается для устройств, способных шифрование диска|



