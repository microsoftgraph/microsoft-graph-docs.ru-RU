---
title: Работа с Intune в Microsoft Graph
description: API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью портала Azure.
author: rolyon
ms.localizationpriority: high
ms.prod: intune
ms.openlocfilehash: 835cdb2e15f942b1adef688e58cea6bd4e83879c
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044815"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.

Все бета-версии API Microsoft Graph для Intune тестируются и проверяются группой Intune до их развертывания. Последние изменения API см. в [журнале изменений](/graph/changelog).

## <a name="using-the-microsoft-graph-api-for-intune"></a>Использование API Microsoft Graph для Intune

Intune предоставляет данные для Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям. С помощью Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемые в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.     

В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя. 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Использование разрешений Microsoft Graph

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune. Как правило, разрешения указываются на портале Azure Active Directory. Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](/graph/permissions-reference).

## <a name="interaction-between-microsoft-graph-apis-for-windows-updates"></a>Взаимодействие между API Microsoft Graph для обновлений Windows

Microsoft Graph включает два набора API, которые можно использовать для управления обновлениями Windows: 

- [API Intune](/graph/intune-concept-overview)
- [API обновлений Windows](/graph/windowsupdates-concept-overview)

Вы можете использовать любой API для управления обновлениями Windows. Однако эти два API несовместимы друг с другом. Каждый из них может переписывать конфигурацию, созданную другим API, не отображая это действие. Использование обоих API для управления обновлениями может привести к неожиданным действиям, в том числе к отмене или изменению временной конфигурации для развертывания обновлений без идентифицированной причины.

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте, [как использовать Azure AD](/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.
- Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.
