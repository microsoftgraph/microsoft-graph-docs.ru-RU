---
title: тип enum fileVaultState
description: Состояние FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 942612457d21b587ccfcfff8720216ade2e1be72
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795552"
---
# <a name="filevaultstate-enum-type"></a>тип enum fileVaultState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние FileVault

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|success|0|Успех состояния FileVault|
|driveEncryptedByUser|1|FileVault включен пользователем и не управляется политикой|
|userDeferredEncryption|2|Политика FileVault успешно установлена, но пользователь еще не начал шифрование|
|escrowNotEnabled|4 |Escrow ключа восстановления FileVault не включен|



