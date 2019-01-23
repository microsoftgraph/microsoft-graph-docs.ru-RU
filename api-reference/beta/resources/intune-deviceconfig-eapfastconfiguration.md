---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399390"
---
# <a name="eapfastconfiguration-enum-type"></a>Тип перечисления eapFastConfiguration

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доступные параметры для конфигурации EAP-FAST.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noProtectedAccessCredential|0|Используйте EAP-FAST без безопасного доступа (PAC).|
|useProtectedAccessCredential|1|Использование защиты безопасного доступа (PAC).|
|useProtectedAccessCredentialAndProvision|2|Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.|




