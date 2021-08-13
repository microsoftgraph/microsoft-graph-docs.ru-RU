---
title: Изучите использование Graph API Azure AD
description: Описывает, как Azure Active Directory API azure AD для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: fbd75626e03cbd4c433a7fa955aa0bc476ed76e6375261bb3bad9d32409302c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216394"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Изучите использование Graph API Azure AD

Это шаг 2 процесса [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)

При планировании миграции в Microsoft Graph время, чтобы просмотреть существующее приложение и каталогизировать API Azure AD Graph, которые вы используете в настоящее время.

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

