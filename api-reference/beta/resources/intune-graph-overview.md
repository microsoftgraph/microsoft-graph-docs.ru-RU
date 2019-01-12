---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 1db77aceaab82e869fc540d2b29cce17ddba100f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911954"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

Для сценариев мобильных устройств management (MDM) Microsoft Graph API для Intune поддерживает развертывание автономных; Intune [гибридные развертывания](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) не поддерживаются. 

## <a name="using-the-microsoft-graph-api-for-intune"></a>С помощью Microsoft Graph API для Intune

Intune предоставляет данные в Microsoft Graph так же, как прочие облачные службы, с расширенными возможностями сущности сведения и отношения навигации.Используйте Microsoft Graph для объединения данных из других служб и Intune создавать полнофункциональный приложения кросс service для ИТ-специалистов и конечных пользователей.     

В следующем примере показано, как определить, установлено ли приложение на устройстве пользователя: 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>С помощью Microsoft Graph разрешения

Графическое представление корпорацию Майкрософт управляет доступом к ресурсам с помощью разрешений. Являясь разработчиком необходимо указать разрешения, необходимые для доступа к ресурсам Intune. Как правило укажите разрешения на портале Azure Active Directory. Для получения дополнительных сведений см [Microsoft Graph разрешения](https://docs.microsoft.com/en-us/graph/permissions-reference).

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, [как использовать Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) для доступа к Microsoft Graph API для Intune.  
- Изучите [Примеры PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), которой показано, как использовать Microsoft Graph API для Intune в контексте рабочие примеры.

