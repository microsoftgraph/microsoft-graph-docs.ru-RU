---
title: тип enum keyStorageProviderOption
description: Параметры импорта служба хранилища поставщика (KSP).
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9f8f47384333189f80d6443a17027e62b1a1e465
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030006"
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



