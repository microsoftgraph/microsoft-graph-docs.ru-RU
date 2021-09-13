---
title: тип enum macOSFileVaultRecoveryKeyTypes
description: Типы ключей восстановления для macOS FileVault
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c7f3d6fc43c38e2d5c51c909d64b0421230e876a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106170"
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
|institutionalRecoveryKey|1|Ключ институционального восстановления похож на "мастерский" ключ восстановления, который можно использовать для разблокировки любого устройства, пароль которого был потерян.|
|personalRecoveryKey|2|Личный ключ восстановления — это уникальный код, который можно использовать для разблокировки устройства пользователя, даже если пароль устройства потерян.|



