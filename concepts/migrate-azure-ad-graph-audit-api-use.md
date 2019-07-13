---
title: Изучение использования приложений API Azure AD Graph
description: Сведения о том, как выполнять аудит API Azure Active Directory (Azure AD) для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14cc61039d97fa43f64599310cf86cce6c348fb2
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645250"
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
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
