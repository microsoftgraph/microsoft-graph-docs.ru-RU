---
title: тип enum eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 880d5b3456f07d8df495b56adece254aa8e5e317
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795237"
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
|useProtectedAccessCredential|1|Использование учетных данных с защищенным доступом (PAC).|
|useProtectedAccessCredentialAndProvision|2|Используйте учетные данные защищенного доступа (PAC) и PAC provision.|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Используйте учетные данные с защищенным доступом (PAC), Provision PAC и сделайте это анонимно.|



