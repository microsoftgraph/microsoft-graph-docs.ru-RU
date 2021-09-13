---
title: расширенный тип enumBitLockerState
description: Состояние Advanced BitLocker
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad5532d92b16fe99be8f0e114e967305324bfcb4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020436"
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



