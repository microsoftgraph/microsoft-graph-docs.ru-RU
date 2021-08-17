---
title: расширенный тип enumBitLockerState
description: Состояние Advanced BitLocker
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 777f2c3b5d530694eb1a5bad6f4b51be445592ad88109661866a1a77bbe20300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54179174"
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
|noUserConsent|1 |Пользователь никогда не давал согласия на шифрование|
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




