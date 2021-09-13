---
title: тип enum fileVaultState
description: Состояние FileVault
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1d9e037eb75fa331e082db5ca19e213c91a927c8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075496"
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



