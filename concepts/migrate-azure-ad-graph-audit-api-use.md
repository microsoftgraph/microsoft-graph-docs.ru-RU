---
title: Изучение использования приложений API Azure AD Graph
description: Сведения о том, как выполнять аудит API Azure Active Directory (Azure AD) для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 405c68d1e0f88af33caa7b5f4c083bd1acdec82d
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872966"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Изучение использования приложений API Azure AD Graph

Это шаг 2 [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

При планировании миграции в Microsoft Graph необходимо проанализировать существующее приложение и каталогизировать используемые API Graph Azure AD Graph.

Сравните список с известными отличиями.  Это помогает определить конкретные изменения, которые необходимо выполнить для переноса приложения.  К ним относятся простые изменения, которые легко разрешить с помощью функций поиска и замены в редакторе или более сложных обновлений, которые могут потребовать большего анализа.

Microsoft Graph поддерживает многие функции и возможности Azure AD Graph.  Существует несколько ключевых отличий.

- [Различия в запросах](migrate-azure-ad-graph-request-differences.md)
- [Функциональные различия](migrate-azure-ad-graph-feature-differences.md)
- [Различия между типами ресурсов](migrate-azure-ad-graph-resource-differences.md)
- [Различия свойств](migrate-azure-ad-graph-property-differences.md)
- [Различия в методах](migrate-azure-ad-graph-method-differences.md)

Кроме того, необходимо проверить разрешения, необходимые для функций, которые использует ваше приложение.  В некоторых случаях доступны более детализированные разрешения.

Дополнительные сведения см. в статье [Разрешения](permissions-reference.md).

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [регистрации приложений, разрешениях и различиях](migrate-azure-ad-graph-app-registration.md) между Azure AD Graph и Microsoft Graph.
- Снова просмотрите [Контрольный список](migrate-azure-ad-graph-planning-checklist.md) .

