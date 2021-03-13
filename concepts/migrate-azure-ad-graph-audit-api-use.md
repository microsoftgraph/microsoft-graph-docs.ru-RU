---
title: Изучение использования приложений API Azure AD Graph
description: Описывает, как аудит API Azure Active Directory (Azure AD) для переноса приложения в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: e7e21f03cdfd8ce3d45f0201d15ec489c7322530
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760695"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a>Изучение использования приложений API Azure AD Graph

Это шаг 2 процесса [миграции приложений.](migrate-azure-ad-graph-planning-checklist.md)

При планировании переноса в Microsoft Graph необходимо время, чтобы просмотреть существующее приложение и каталогизировать API Azure AD Graph, которые вы используете в настоящее время.

Сравните список с известными различиями.  Это помогает определить конкретные изменения, которые необходимо внести для переноса приложения.  К ним относятся простые изменения, которые легко разрешить с помощью функций поиска и замены редактора или более сложные обновления, которые могут потребовать дополнительного анализа.

Microsoft Graph поддерживает многие из тех же функций и возможностей диаграммы Azure AD.  Существует несколько ключевых отличий:

- [Различия запросов](migrate-azure-ad-graph-request-differences.md)
- [Функциональные различия](migrate-azure-ad-graph-feature-differences.md)
- [Различия в типах ресурсов](migrate-azure-ad-graph-resource-differences.md)
- [Различия свойств](migrate-azure-ad-graph-property-differences.md)
- [Различия метода](migrate-azure-ad-graph-method-differences.md)

Кроме того, необходимо проверить разрешения, необходимые для функций, которые использует приложение.  В некоторых случаях доступны дополнительные разрешения на детализацию.

Дополнительные сведения см. в статье [Разрешения](permissions-reference.md).

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о различиях в регистрации [приложений, разрешениях](migrate-azure-ad-graph-app-registration.md) и согласии между Azure AD Graph и Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.

