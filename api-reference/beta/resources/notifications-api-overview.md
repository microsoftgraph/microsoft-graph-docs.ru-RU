---
title: Использование уведомлений о API-Интерфейс REST в Microsoft Graph
description: Уведомления о API в Microsoft Graph можно использовать для отправки push-уведомления для пользователя. Просто целевого учетная запись пользователя, чтобы отправить уведомление и платформы будет доставки уведомления для всех конечных точек устройства. Уведомления о API запросы выполняются от имени пользователя с помощью делегированных разрешений и [разрешений уведомлений]( /graph/permissions_reference), который можно использовать с любого из учетных записей Майкрософт или рабочего или школы учетных записей.
localization_priority: Priority
ms.openlocfilehash: 04787cb9a9b589036020651934041b4fc399adb1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853027"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Использование уведомлений о API-Интерфейс REST в Microsoft Graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Уведомления о API в Microsoft Graph можно использовать для отправки push-уведомления для пользователя. Просто целевого учетная запись пользователя, чтобы отправить уведомление и платформы будет доставки уведомления для всех конечных точек устройства. Уведомления о API запросы выполняются от имени пользователя с помощью [делегированных разрешений](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) и [разрешений уведомлений]( /graph/permissions_reference), который можно использовать с любого из учетных записей Майкрософт или рабочего или школы учетных записей.
Этот тип уведомления, ориентированные на пользователя представлены [уведомлений](../resources/projectrome-notification.md) ресурсов и сохраняются в Microsoft Graph. Его можно затем получить доступ и управляют публикации приложения через [Project рим пакет SDK для API -интерфейсы](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Дальнейшие действия
- Просмотр [уведомлений ресурсов](../resources/projectrome-notification.md) и создание уведомлений для работы с вашими пользователями. 
- опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
