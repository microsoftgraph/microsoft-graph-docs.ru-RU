---
title: Изучите использование Graph API Azure AD
description: Описывает, как Azure Active Directory (Azure AD) Graph API для переноса приложения в API microsoft Graph.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: d6a440e71350433feacc1a92fbc6928523c0b534
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077630"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Изучите использование Graph API Azure AD

Это шаг 2 процесса [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)

При планировании миграции в Microsoft Graph время, чтобы просмотреть существующее приложение и каталогизировать Azure Active Directory (Azure AD) Graph API, которые вы используете в настоящее время.

Сравните список с известными различиями.  Это помогает определить конкретные изменения, которые необходимо внести для переноса приложения.  К ним относятся простые изменения, которые легко разрешить с помощью функций поиска и замены редактора или более сложные обновления, которые могут потребовать дополнительного анализа.

Microsoft Graph поддерживает многие из тех же функций и возможностей графа Azure AD.  Существует несколько ключевых отличий:

- [Различия запросов](migrate-azure-ad-graph-request-differences.md)
- [Функциональные различия](migrate-azure-ad-graph-feature-differences.md)
- [Различия в типах ресурсов](migrate-azure-ad-graph-resource-differences.md)
- [Различия свойств](migrate-azure-ad-graph-property-differences.md)
- [Различия метода](migrate-azure-ad-graph-method-differences.md)

Кроме того, необходимо проверить разрешения, необходимые для функций, которые использует приложение.  В некоторых случаях доступны дополнительные разрешения на детализацию.

Дополнительные сведения см. в статье [Разрешения](permissions-reference.md).

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о различиях в регистрации [приложений,](migrate-azure-ad-graph-app-registration.md) разрешениях и согласиях между Azure AD Graph и Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.

