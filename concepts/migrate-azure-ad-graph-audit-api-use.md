---
title: Изучите Azure Active Directory (Azure AD) Graph использования приложений API
description: Описывает, как Azure Active Directory (Azure AD) Graph API для переноса приложения в API microsoft Graph.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 8386c3c77a5f42115236875d8405f97c5f49ff42
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139172"
---
# <a name="examine-azure-active-directory-azure-ad-graph-apis-app-usage"></a>Изучите Azure Active Directory (Azure AD) Graph использования приложений API

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

