---
title: Тип перечисления keyStorageProviderOption
description: Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424226"
---
# <a name="keystorageprovideroption-enum-type"></a>Тип перечисления keyStorageProviderOption

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры импорта хранилища ключей поставщика (поставщика хранилища КЛЮЧЕЙ).

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Импорта для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — импорт поставщика хранилища КЛЮЧЕЙ программного обеспечения.|
|useTpmKspOtherwiseFail|1|Импорт для доверенного платформы модуля (TPM) поставщика хранилища КЛЮЧЕЙ, если этот параметр указан, в противном случае — не удается.|
|usePassportForWorkKspOtherwiseFail|2|Импорт Passport для работы поставщика хранилища КЛЮЧЕЙ Если доступно, в противном случае — ошибка.|
|useSoftwareKsp|3|Импорт на программное обеспечение поставщика хранилища КЛЮЧЕЙ.|




