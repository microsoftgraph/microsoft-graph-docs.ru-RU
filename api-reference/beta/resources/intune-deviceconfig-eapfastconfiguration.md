---
title: тип enum eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cd64a51bc9e41c1ea558ad4d1245b693de29f3c7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069189"
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



