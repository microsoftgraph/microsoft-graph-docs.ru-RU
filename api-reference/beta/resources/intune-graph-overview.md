---
title: Использование API Graph для Intune — API Microsoft Graph
description: Перечисление API Microsoft Graph для коечных точек Intune (REST), которые можно использовать для управления организацией клиента, его устройствами, приложениями, доступом и ресурсами.
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 3b479617ce476492ca716db7742f1e10aab88b18
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225055"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются. 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Использование API Microsoft Graph для Intune

Intune предоставляет данные для Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.С помощью Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемые в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.     

В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя. 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Использование разрешений Microsoft Graph

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune. Как правило, разрешения указываются на портале Azure Active Directory. Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, [как использовать Azure AD](https://docs.microsoft.com/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.  
- Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.

