---
title: тип enum keyStorageProviderOption
description: Параметры импорта служба хранилища поставщика (KSP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7bfd89c8e74264aca79af72325d6b5b4a96b23a3a3fadd44b32c94f3fa95cc58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219754"
---
# <a name="keystorageprovideroption-enum-type"></a>тип enum keyStorageProviderOption

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры импорта служба хранилища поставщика (KSP).

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Импортировать в доверенный модуль платформы (TPM) KSP, если он присутствует, в противном случае импортировать в программное обеспечение KSP.|
|useTpmKspOtherwiseFail|1 |Импорт в доверенный модуль платформы (TPM) KSP, если он присутствует, в противном случае не удается.|
|usePassportForWorkKspOtherwiseFail|2|Импорт в Passport для работы KSP при наличии, в противном случае сбой.|
|useSoftwareKsp|3 |Импорт в программное обеспечение KSP.|




