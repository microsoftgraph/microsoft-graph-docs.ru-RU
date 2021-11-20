---
title: Работа с облачными ПК с ОС Windows 365 с использованием программного интерфейса Microsoft Graph
description: API microsoft Graph программный доступ к сведениям о облачных КОМПЬЮТЕРАх и действиям по управлению в организации.
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 566c2e37c2b6ca6f36b6ef41d3f2911fc0539a6f
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123734"
---
# <a name="working-with-windows-365-cloud-pcs-using-the-microsoft-graph-api"></a>Работа с облачными ПК с ОС Windows 365 с использованием программного интерфейса Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows 365 — это облачная служба, которая автоматически создает новый тип виртуальной машины Windows (облачные компьютеры) для пользователей. Каждый облачный компьютер назначен отдельному пользователю в качестве Windows устройства. Windows 365 предоставляет реализованные в Microsoft 365 преимущества производительности, безопасности и совместной работы.

API microsoft Graph программный доступ к сведениям о облачных КОМПЬЮТЕРАх и действиям по управлению в организации. API выполняет те же операции, что и доступные через Microsoft Endpoint Manager. 

> [!IMPORTANT]
> Для использования API Graph Microsoft для облачных компьютеров требуется активная лицензия [Windows 365](https://www.microsoft.com/windows-365) для организации. В настоящее время API Graph Microsoft доступен для Windows 365 Enterprise и не Windows 365 Business. 

## <a name="using-the-microsoft-graph-api-for-cloud-pcs"></a>Использование API Graph Microsoft для облачных компьютеров

С помощью microsoft Graph вы можете закадровку и управление облачными компьютерами в вашей организации. Если используется совместно с API Intune, вы также можете управлять облачными компьютерами наряду с физическими конечными точками. 

## <a name="using-microsoft-graph-permissions"></a>Использование разрешений Microsoft Graph

Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения. Как разработчик необходимо указать разрешения, необходимые для доступа Windows 365 ресурсов. Как правило, разрешения указываются на портале Azure Active Directory. Дополнительные сведения см. в [статье Microsoft Graph разрешений и](/graph/permissions-reference) перейдите в раздел Разрешения облачных [ПК.](/graph/permissions-reference#cloud-pc-permissions) 

## <a name="common-use-cases"></a>Основные варианты использования

|Варианты использования|Ресурсы REST|См. также|
|:---|:---|:---|
|Список, создание, обновление, удаление или назначение политик провизии|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|[Обзор подготовка](/windows-365/enterprise/provisioning)|
|Управление облачными компьютерами, включая перепроизводение, конечный период льготы для облачных ПК, массовое перепроизводение и повторное создание облачных компьютеров|[cloudPC](../resources/cloudpc.md)|[Жизненный цикл облачных компьютеров](/windows-365/enterprise/lifecycle)|
|Список, получить, создать, удалить, получить исходные изображения и перезагрузить изображения облачной ОС ПК|[cloudPCDeviceImage](../resources/cloudpcdeviceimage.md)|[Обзор изображений устройств](/windows-365/enterprise/device-images)|
|Список, создание, удаление, обновление, обновление пароля домена AD и проверка состояния локальной сети|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|[Обзор локального сетевого подключения](/windows-365/enterprise/on-premises-network-connections)|
|Список событий аудита для облачных компьютеров, получения определенного события аудита и получения типов действий аудита|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|[Получить журналы аудита облачных ПК](/windows-365/enterprise/get-cloud-pc-audit-logs-using-powershell)|
|Список, получить, создать, обновить, удалить или назначить параметры пользователей|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|[Обзор параметров пользователей](../resources/cloudpcusersetting.md)|

## <a name="whats-new"></a>Новые возможности

Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
- Ознакомьтесь с [обзором Windows 365 cloud PC в Microsoft Graph.](/graph/cloudpc-concept-overview)
- Попробуйте Windows API облачных ПК 365 с помощью [Microsoft Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer)