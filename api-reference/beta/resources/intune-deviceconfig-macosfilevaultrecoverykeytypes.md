---
title: тип enum macOSFileVaultRecoveryKeyTypes
description: Типы ключей восстановления для macOS FileVault
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c92bec5d4ad5f94e6990c537defe7eb6488b4694bc3f3a5bb4483c716dcaa19d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54198327"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a>тип enum macOSFileVaultRecoveryKeyTypes

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Типы ключей восстановления для macOS FileVault

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Значение устройства по умолчанию, без намерения.|
|institutionalRecoveryKey|1 |Ключ институционального восстановления похож на "мастерский" ключ восстановления, который можно использовать для разблокировки любого устройства, пароль которого был потерян.|
|personalRecoveryKey|2|Личный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя, даже если пароль устройства потерян.|




