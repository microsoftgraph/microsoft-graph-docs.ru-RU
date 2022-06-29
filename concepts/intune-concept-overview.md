---
title: Обзор API устройств и приложений Intune
description: Используйте Intune API в Microsoft Graph для управления устройствами и приложениями Intune и автоматизации в своей организации. Независимые поставщики программного обеспечения могут использовать Intune API для управления клиентами пользователей.
author: dougeby
ms.localizationpriority: high
ms.prod: intune
ms.openlocfilehash: 30da93fa91101f5ef49ca5bed64a7c1b71fa73db
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444889"
---
# <a name="intune-devices-and-apps-api-overview"></a>Обзор API устройств и приложений Intune

Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации. С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства. 

Если вы независимый поставщик программного обеспечения, вы также можете использовать API Intune для управления клиентами.

> [!VIDEO https://www.youtube-nocookie.com/embed/yU1HeqNmN7A]

## <a name="why-integrate-with-intune"></a>Преимущества интеграции с Intune

Вы также можете использовать API Intune в Microsoft Graph для доступа к сведениям об устройствах и приложениях из Intune, управления приложениями и автоматизации Intune.

### <a name="manage-devices"></a>Управление устройствами

С помощью API Intune вы можете:

- Определять и применять политики [соответствия устройств различным требованиям](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem), таким как сложность и длина пароля, шифрование, уровни защиты от угроз.  (То, поддерживается ли политика, зависит от используемой операционной системы и ее версии.)
- [Защищать данные компании](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy) независимо от платформы устройства (Windows, Android, Mac или iOS).
- Создавать и развертывать политики [конфигурации устройств](/graph/api/resources/intune-deviceconfig-deviceconfiguration), включая платформы и версии операционной системы, членство в доменах и управление параметрами конфигурации.
- Создавать и развертывать политики [контроля доступа](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings) для устройств, включая ограниченную загрузку, доступ к сетевым аксессуарам и передачу данных.
- Выполнять [удаленные действия](/graph/api/resources/intune-devices-manageddevice), например поиск устройства, изменение пароля и стирание данных устройства.

### <a name="manage-apps"></a>Управление приложениями 

С помощью API Intune вы можете выполнять указанные ниже задачи по управлению приложениями.

- Развертывание [приложений на устройствах](/graph/api/resources/intune-apps-mobileapp) и запрет развертывания приложений.
- Управление доступом к [электронным книгам](/graph/api/resources/intune-books-ebookinstallsummary) и соответствующим службам.
- Определение и развертывание параметров конфигурации и защиты приложений, а также политик их использования.

### <a name="automate-intune"></a>Автоматизация Intune

Автоматизируйте Intune, используя API Intune для:

- определения и назначения правил доступа [на основе ролей](/graph/api/resources/intune-rbac-conceptual);
- аудита и создания отчетов о соответствии требованиям, использовании и доступе;
- управления [затратами на телекоммуникации](/graph/api/resources/intune-tem-conceptual).

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API Intune в Microsoft Graph 1.0](/graph/api/resources/intune-graph-overview?view=graph-rest-1.0&preserve-view=true)
- [API Intune в бета-версии Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Дальнейшие действия

- [Доступ к интерфейсам API Intune в Microsoft Graph с использованием Azure AD](/intune/intune-graph-apis).
- Узнайте, как выполнять распространенные задачи, с помощью [примеров PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples).
- Узнайте, как [использовать REST API Intune](/graph/api/resources/intune-graph-overview).
- Сведения о новых возможностях API Intune см. в [журнале изменений](changelog.md).
- Изучите [ресурсы](https://developer.microsoft.com/graph/gallery/) с новыми идеями о том, как использовать Microsoft Graph.
