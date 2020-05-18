(function ($) {
  'use strict';

// flot chart hospital patient total
    var totalSalaryData = {
      labels: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
      datasets: [{
        label: '# of Votes',
        data: [15000, 13000, 5000, 13000, 18000, 21000, 24000, 22000, 19000, 14000, 14000, 14000],
        backgroundColor: [
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',

        ],
        borderColor: [
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          '#5e6eed',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',
          'rgba(94, 110, 237, .3)',
        ],
        borderWidth: 1,
        fill: false
      }]
    };

    var totalSalaryOptions = {
      scales: {
        yAxes: [{
          ticks: {
            display: true,
            min: 0,

            callback: function(label, index, labels) {
              return label/1000+'k';
            }
          },
          gridLines: {
            display: true,
            color: "rgba(169, 169, 169, .32)",
            drawBorder: false,
            zeroLineColor: "rgba(169, 169, 169, .32)",
          },
          beginAtZero: true
        }],
        xAxes: [{
          barPercentage: 0.4,
          gridLines: {
            drawBorder: false,
            display: false,
            drawBorder: false,
          }
        }]
      },
      legend: {
        display: false
      },
      elements: {
        point: {
          radius: 0
        }
      }

    };

    if ($("#totalSalary").length) {
      var totalSalaryCanvas = $("#totalSalary").get(0).getContext("2d");
      // This will get the first returned node in the jQuery collection.
      var totalSalary = new Chart(totalSalaryCanvas, {
        type: 'bar',
        data: totalSalaryData,
        options: totalSalaryOptions
      });
    }
    $(".close-hr-banner").on("click", function() {
      $('.hr-banner').hide();
    });

})(jQuery);
