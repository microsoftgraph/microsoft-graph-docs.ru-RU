---
title: Обзор API облачной среды универсальной печати
description: Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.
author: braedenp-msft
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 84a8a97315bb8ca62afb22f76db06fa67fb4e307
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557866"
---
# <a name="universal-print-cloud-printing-api-overview"></a>Обзор API облачной среды универсальной печати

Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы от Майкрософт.

![Снимок экрана с изображением главной страницы универсальной печати на портале Azure](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a>Зачем нужна универсальная печать?

Универсальная печать — это функции печати Windows Server, перенесенные в облако Microsoft 365, благодаря которым организации теперь могут обойтись без локальных серверов печати и не устанавливать драйверы печати на устройствах. Кроме того, в рамках универсальной печати предусмотрены дополнительные функции, например, группы безопасности для доступа к принтеру, обнаружение принтеров на основе расположения и расширенными возможностями для администраторов.

По мере внедрения универсальной печати в организациях организации и независимые поставщики программного обеспечения могут использовать API универсальной печати в Microsoft Graph, чтобы создавать и расширять приложения для поддержки новых сценариев.

### <a name="print-documents-from-web-and-mobile-applications"></a>Печать документов из веб-приложений и мобильных приложений

Благодаря перемещению инфраструктуры печати в облако печатать документы можно непосредственно из веб-приложений и мобильных приложений.

Чтобы приступить к работе с API универсальной печати, выполните указанные ниже действия.

1. [Создайте задание печати](/graph/api/printer-post-jobs?view=graph-rest-beta) и сохраните идентификатор полученного документа.
2. [Отправьте данные документа](/graph/api/printdocument-uploaddata?view=graph-rest-beta) в документ.
3. [Запустите задание печати](/graph/api/printjob-startprintjob?view=graph-rest-beta).

### <a name="manage-printers"></a>Управление принтерами

Отследить принтеры организации, настройки принтеров и их использование — непростая задача. Благодаря API универсальной печати можно интегрировать эти три направления.

* **Отслеживать состояние принтеров, их настройки и доступность**можно через [Список принтеров](/graph/api/print-list-printers?view=graph-rest-beta) и [printerStatus](/graph/api/resources/printerstatus?view=graph-rest-beta).

* **Узнать, кто из пользователей использует принтеры и сколько страниц они печатают** можно через отчетные API:
  * [Список dailyPrintUsageSummariesByUser](/graph/api/reportroot-list-dailyprintusagesummariesbyuser?view=graph-rest-beta)
  * [Список monthlyPrintUsageSummariesByUser](/graph/api/reportroot-list-monthlyprintusagesummariesbyuser?view=graph-rest-beta)
  * [Список dailyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-dailyprintusagesummariesbyprinter?view=graph-rest-beta)
  * [Список monthlyPrintUsageSummariesByPrinter](/graph/api/reportroot-list-monthlyprintusagesummariesbyprinter?view=graph-rest-beta)

* **Настройка разрешений для пользователей** через изменения в членстве пользователей и групп касательно принтеров:
  * [Список allowedUsers](/graph/api/printer-list-allowedusers?view=graph-rest-beta)
  * [Добавление allowedUser](/graph/api/printer-post-allowedusers?view=graph-rest-beta)
  * [Удаление allowedUser](/graph/api/printer-delete-alloweduser?view=graph-rest-beta)
  * [Список allowedGroups](/graph/api/printer-list-allowedgroups?view=graph-rest-beta)
  * [Добавление allowedGroup](/graph/api/printer-post-allowedgroups?view=graph-rest-beta)
  * [Удаление allowedGroup](/graph/api/printer-delete-allowedgroup?view=graph-rest-beta)

### <a name="seamlessly-replace-or-update-printer-hardware"></a>Комфорт при замене и обновлении оборудования для печати

Принтеры не видны пользователям до момента, когда они получают к ним [доступ](/graph/api/print-post-printershares?view=graph-rest-beta). Это позволяет администраторам детально контролировать доступность определенного оборудования для печати в определенный момент времени.

При общем доступе к принтеру создается ресурс [printerShare](/graph/api/resources/printershare?view=graph-rest-beta), который в любой момент можно обновить для перевода на другой принтер, что упрощает замену неисправного оборудования для печати и отправку принтеров в текущий ремонт.

Чтобы применить эту возможность в своем приложении, перейдите в [Обновление printerShare](/graph/api/printershare-update?view=graph-rest-beta) и обновите ссылку `printer` на printerShare.

## <a name="api-reference"></a>Справочные материалы по API
Ищете справочные материалы по API для этой службы?

- [API универсальной печати в бета-версии Microsoft Graph](/graph/api/resources/print?view=graph-rest-beta)

## <a name="see-also"></a>См. также

- [Что такое универсальная печать](https://docs.microsoft.com/universal-print/fundamentals/universal-print-whatis)
- Мы будем рады узнать ваше мнение об API универсальной печати через [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)!
