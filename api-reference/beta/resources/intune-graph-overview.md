---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079653"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

В сценариях управления мобильными устройствами (MDM) API Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются. 

## <a name="using-the-intune-graph-api"></a>Использование API Graph для Intune

Intune предоставляет данные в Microsoft Graph так же, как прочие облачные службы, с расширенными возможностями сущности сведения и отношения навигации.Используйте Microsoft Graph для объединения данных из других служб и Intune создавать полнофункциональный приложения кросс service для ИТ-специалистов и конечных пользователей.     

Ниже приведен пример того, как определить, установлено ли приложение на устройстве пользователя. 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a>С помощью области разрешений график

Графическое представление корпорацию Майкрософт управляет доступом к ресурсам, с помощью области разрешений. Разработчикам необходимо указать области разрешений, необходимые для доступа к ресурсам Intune. Как правило, требуемые области разрешений указываются на портале Azure Active Directory. Дополнительные сведения см. в статье об [областях разрешений в Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) и [областях разрешений в Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a>Чтобы использовать содержания на сайте Microsoft Graph
  
Поиск частей документацию по API графике Intune и ресурсов, чтобы увидеть могут просматривать содержание (в левой панели веб-сайта).

1. Щелкните **Ссылку /Beta** , чтобы открыть документы бета-версии.
2. Прокрутите список вниз и выберите **Intune**.
3. Продолжайте щелкать элемент для части API-интерфейса подразделах ниже **Intune** вы 
