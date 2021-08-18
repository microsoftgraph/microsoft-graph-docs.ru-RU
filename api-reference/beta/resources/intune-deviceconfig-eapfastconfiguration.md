---
title: тип enum eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3f3f6db981d29c2150beba9d391180248c9151188d97b2b6810cf6ae13e19285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227471"
---
# <a name="eapfastconfiguration-enum-type"></a>тип enum eapFastConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доступные параметры для конфигурации EAP-FAST.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noProtectedAccessCredential|0|Используйте EAP-FAST без защищенных учетных данных доступа (PAC).|
|useProtectedAccessCredential|1 |Использование учетных данных с защищенным доступом (PAC).|
|useProtectedAccessCredentialAndProvision|2|Используйте учетные данные защищенного доступа (PAC) и PAC provision.|
|useProtectedAccessCredentialAndProvisionAnonymously|3 |Используйте учетные данные с защищенным доступом (PAC), Provision PAC и сделайте это анонимно.|




