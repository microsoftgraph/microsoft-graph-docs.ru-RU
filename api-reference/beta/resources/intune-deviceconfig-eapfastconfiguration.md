---
title: Тип перечисления eapFastConfiguration
description: Доступные параметры для конфигурации EAP-FAST.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954458"
---
# <a name="eapfastconfiguration-enum-type"></a>Тип перечисления eapFastConfiguration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Доступные параметры для конфигурации EAP-FAST.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|noProtectedAccessCredential|0|Используйте EAP-FAST без безопасного доступа (PAC).|
|useProtectedAccessCredential|1|Использование защиты безопасного доступа (PAC).|
|useProtectedAccessCredentialAndProvision|2|Использование защищенного доступа учетные данные (PAC) и подготовки идентификационные|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Использование защищенного доступа учетные данные (PAC), PAC подготовки и делать это анонимного доступа.|





