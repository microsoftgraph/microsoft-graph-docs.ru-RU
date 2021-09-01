---
title: тип enum keyStorageProviderOption
description: Параметры импорта служба хранилища поставщика (KSP).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6dc213f3cef76380a5bf40d91b6220e1408783f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786279"
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
|useTpmKspOtherwiseFail|1|Импорт в доверенный модуль платформы (TPM) KSP, если он присутствует, в противном случае не удается.|
|usePassportForWorkKspOtherwiseFail|2|Импорт в Passport для работы KSP при наличии, в противном случае сбой.|
|useSoftwareKsp|3|Импорт в программное обеспечение KSP.|



