---
title: Работа с Intune в Microsoft Graph
description: API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью портала Azure.
author: dougeby
ms.localizationpriority: high
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 974e83fb042605232a49383db8e808a916b0a54d
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044780"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются. 



## <a name="using-the-microsoft-graph-api-for-intune"></a>Использование API Microsoft Graph для Intune

Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.  API Microsoft Graph используется для объединения сведений из других служб и Intune, чтобы создавать функциональные приложения, работающие с несколькими службами, для ИТ-специалистов или пользователей.     

В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя. 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a>Доступ к API Microsoft Graph для Intune

Intune поддерживает как [делегированные разрешения](/graph/auth-v2-user), так и [разрешения приложений](/graph/auth-v2-service). Делегированные разрешения и разрешения приложений поддерживают операции как чтения, так и записи. Разрешения приложений и делегированные разрешения поддерживает как однотенантные, так и многотенантные приложения. Дополнительные сведения о разрешениях, доступных в Microsoft Graph, см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference).

## <a name="using-permissions"></a>Использование разрешений

API Microsoft Graph контролирует доступ к ресурсам с помощью разрешений. Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune. Как правило, разрешения указываются на портале Azure Active Directory. Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](/graph/permissions-reference).

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
